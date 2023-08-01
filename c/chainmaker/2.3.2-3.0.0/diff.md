# Comparing `tmp/chainmaker-2.3.2.tar.gz` & `tmp/chainmaker-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainmaker-2.3.2.tar", last modified: Thu Jul 13 09:22:08 2023, max compression
+gzip compressed data, was "chainmaker-3.0.0.tar", last modified: Tue Aug  1 08:18:06 2023, max compression
```

## Comparing `chainmaker-2.3.2.tar` & `chainmaker-3.0.0.tar`

### file list

```diff
@@ -1,27 +1,177 @@
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-13 09:22:08.921145 chainmaker-2.3.2/
--rw-r--r--   0 superhin   (502) staff       (20)    11356 2021-09-15 06:14:28.000000 chainmaker-2.3.2/LICENSE
--rw-r--r--   0 superhin   (502) staff       (20)       75 2021-09-15 06:14:28.000000 chainmaker-2.3.2/NOTICE
--rw-r--r--   0 superhin   (502) staff       (20)      303 2023-07-13 09:22:08.920875 chainmaker-2.3.2/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)    18087 2023-02-05 14:05:49.000000 chainmaker-2.3.2/README.md
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-13 09:22:08.917899 chainmaker-2.3.2/chainmaker/
--rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-14 06:15:05.000000 chainmaker-2.3.2/chainmaker/__init__.py
--rw-r--r--   0 superhin   (502) staff       (20)    31827 2023-07-13 07:20:37.000000 chainmaker-2.3.2/chainmaker/chain_client.py
--rw-r--r--   0 superhin   (502) staff       (20)   123645 2023-07-13 07:20:37.000000 chainmaker-2.3.2/chainmaker/chain_manager.py
--rw-r--r--   0 superhin   (502) staff       (20)     3109 2023-06-14 06:15:05.000000 chainmaker-2.3.2/chainmaker/client_node.py
--rw-r--r--   0 superhin   (502) staff       (20)    18670 2023-06-14 06:15:05.000000 chainmaker-2.3.2/chainmaker/client_user.py
--rw-r--r--   0 superhin   (502) staff       (20)     8029 2023-07-13 07:20:37.000000 chainmaker-2.3.2/chainmaker/conn_pool.py
--rw-r--r--   0 superhin   (502) staff       (20)     7824 2023-07-13 07:20:37.000000 chainmaker-2.3.2/chainmaker/exceptions.py
--rw-r--r--   0 superhin   (502) staff       (20)    27242 2023-06-14 06:15:05.000000 chainmaker-2.3.2/chainmaker/keys.py
--rw-r--r--   0 superhin   (502) staff       (20)      184 2023-06-14 06:15:05.000000 chainmaker-2.3.2/chainmaker/node.py
--rw-r--r--   0 superhin   (502) staff       (20)     3685 2023-06-14 06:15:05.000000 chainmaker-2.3.2/chainmaker/payload.py
--rw-r--r--   0 superhin   (502) staff       (20)    19777 2023-06-14 06:15:05.000000 chainmaker-2.3.2/chainmaker/sdk_config.py
--rw-r--r--   0 superhin   (502) staff       (20)      184 2023-06-14 06:15:05.000000 chainmaker-2.3.2/chainmaker/user.py
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-13 09:22:08.920362 chainmaker-2.3.2/chainmaker.egg-info/
--rw-r--r--   0 superhin   (502) staff       (20)      303 2023-07-13 09:22:08.000000 chainmaker-2.3.2/chainmaker.egg-info/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)      500 2023-07-13 09:22:08.000000 chainmaker-2.3.2/chainmaker.egg-info/SOURCES.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2023-07-13 09:22:08.000000 chainmaker-2.3.2/chainmaker.egg-info/dependency_links.txt
--rw-r--r--   0 superhin   (502) staff       (20)       86 2023-07-13 09:22:08.000000 chainmaker-2.3.2/chainmaker.egg-info/requires.txt
--rw-r--r--   0 superhin   (502) staff       (20)       11 2023-07-13 09:22:08.000000 chainmaker-2.3.2/chainmaker.egg-info/top_level.txt
--rw-r--r--   0 superhin   (502) staff       (20)      103 2021-09-15 06:14:28.000000 chainmaker-2.3.2/pyproject.toml
--rw-r--r--   0 superhin   (502) staff       (20)       38 2023-07-13 09:22:08.921279 chainmaker-2.3.2/setup.cfg
--rw-r--r--   0 superhin   (502) staff       (20)     1630 2023-07-13 07:32:19.000000 chainmaker-2.3.2/setup.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.430688 chainmaker-3.0.0/
+-rw-r--r--   0 superhin   (502) staff       (20)    11356 2021-09-15 06:14:28.000000 chainmaker-3.0.0/LICENSE
+-rw-r--r--   0 superhin   (502) staff       (20)       75 2021-09-15 06:14:28.000000 chainmaker-3.0.0/NOTICE
+-rw-r--r--   0 superhin   (502) staff       (20)      303 2023-08-01 08:18:06.430255 chainmaker-3.0.0/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)    18087 2023-02-05 14:05:49.000000 chainmaker-3.0.0/README.md
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.322688 chainmaker-3.0.0/chainmaker/
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/__init__.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.337023 chainmaker-3.0.0/chainmaker/apis/
+-rw-r--r--   0 superhin   (502) staff       (20)     1153 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/__init__.py
+-rw-r--r--   0 superhin   (502) staff       (20)    15824 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/apis/account_manager.py
+-rw-r--r--   0 superhin   (502) staff       (20)     7527 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/apis/archive_manage.py
+-rw-r--r--   0 superhin   (502) staff       (20)     4608 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/base_client.py
+-rw-r--r--   0 superhin   (502) staff       (20)    22889 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/apis/cert_manage.py
+-rw-r--r--   0 superhin   (502) staff       (20)    71260 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/chain_config.py
+-rw-r--r--   0 superhin   (502) staff       (20)    22489 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/chain_query.py
+-rw-r--r--   0 superhin   (502) staff       (20)     6693 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/chainmaker_server.py
+-rw-r--r--   0 superhin   (502) staff       (20)    37630 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/contract_manage.py
+-rw-r--r--   0 superhin   (502) staff       (20)      123 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/apis/cross_transaction.py
+-rw-r--r--   0 superhin   (502) staff       (20)     8998 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/dpos_distribution.py
+-rw-r--r--   0 superhin   (502) staff       (20)    10371 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/dpos_erc20.py
+-rw-r--r--   0 superhin   (502) staff       (20)     5837 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/dpos_slashing.py
+-rw-r--r--   0 superhin   (502) staff       (20)    19907 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/dpos_stake.py
+-rw-r--r--   0 superhin   (502) staff       (20)     7271 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/apis/multi_sign.py
+-rw-r--r--   0 superhin   (502) staff       (20)    16402 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/apis/private_compute.py
+-rw-r--r--   0 superhin   (502) staff       (20)     5038 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/apis/pubkey_manage.py
+-rw-r--r--   0 superhin   (502) staff       (20)      117 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/apis/relay_cross.py
+-rw-r--r--   0 superhin   (502) staff       (20)     8698 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/apis/subscribe_manage.py
+-rw-r--r--   0 superhin   (502) staff       (20)    31690 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/chain_client.py
+-rw-r--r--   0 superhin   (502) staff       (20)   135451 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/chain_manager.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3109 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/client_node.py
+-rw-r--r--   0 superhin   (502) staff       (20)    18670 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/client_user.py
+-rw-r--r--   0 superhin   (502) staff       (20)     7991 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/conn_pool.py
+-rw-r--r--   0 superhin   (502) staff       (20)     7835 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/exceptions.py
+-rw-r--r--   0 superhin   (502) staff       (20)    27242 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/keys.py
+-rw-r--r--   0 superhin   (502) staff       (20)      184 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/node.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3685 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/payload.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.337480 chainmaker-3.0.0/chainmaker/protos/
+-rw-r--r--   0 superhin   (502) staff       (20)     1238 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/__init__.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.339546 chainmaker-3.0.0/chainmaker/protos/accesscontrol/
+-rw-r--r--   0 superhin   (502) staff       (20)     4993 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/accesscontrol/member_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/accesscontrol/member_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1482 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/accesscontrol/policy_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/accesscontrol/policy_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.340636 chainmaker-3.0.0/chainmaker/protos/api/
+-rw-r--r--   0 superhin   (502) staff       (20)     4291 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/api/rpc_node_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)    25576 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/api/rpc_node_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.348794 chainmaker-3.0.0/chainmaker/protos/common/
+-rw-r--r--   0 superhin   (502) staff       (20)     8954 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/birdsnest_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/birdsnest_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     6741 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/block_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/block_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2772 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/contract_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/contract_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     5663 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/request_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/request_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)    12432 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/result_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/result_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2979 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/rwset_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/rwset_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     4223 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/transaction_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/common/transaction_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.356609 chainmaker-3.0.0/chainmaker/protos/config/
+-rw-r--r--   0 superhin   (502) staff       (20)    14100 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/chain_config_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/chain_config_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2210 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/chainmaker_server_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/chainmaker_server_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3569 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/local_config_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/local_config_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1979 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/log_config_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/log_config_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2154 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/tx_filter_config_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/config/tx_filter_config_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.358614 chainmaker-3.0.0/chainmaker/protos/consensus/
+-rw-r--r--   0 superhin   (502) staff       (20)     9456 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/consensus/consensus_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/consensus/consensus_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.360484 chainmaker-3.0.0/chainmaker/protos/discovery/
+-rw-r--r--   0 superhin   (502) staff       (20)     2402 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/discovery/discovery_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/discovery/discovery_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.362233 chainmaker-3.0.0/chainmaker/protos/net/
+-rw-r--r--   0 superhin   (502) staff       (20)     2259 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/net/net_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/net/net_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.365273 chainmaker-3.0.0/chainmaker/protos/store/
+-rw-r--r--   0 superhin   (502) staff       (20)     2604 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/store/query_result_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/store/query_result_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     8482 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/store/store_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/store/store_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.367042 chainmaker-3.0.0/chainmaker/protos/sync/
+-rw-r--r--   0 superhin   (502) staff       (20)     4549 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/sync/sync_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/sync/sync_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.406496 chainmaker-3.0.0/chainmaker/protos/syscontract/
+-rw-r--r--   0 superhin   (502) staff       (20)     4223 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/account_manager_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/account_manager_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2689 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/archive_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/archive_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1903 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/cert_manage_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/cert_manage_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3443 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/chain_config_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/chain_config_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3151 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/chain_query_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/chain_query_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1339 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/coinbase_manage_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/coinbase_manage_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1803 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/common_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/common_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     8898 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/contract_manage_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/contract_manage_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3819 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/cross_transaction_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/cross_transaction_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1418 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_config_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_config_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1932 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_distribution_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_distribution_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1817 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_erc20_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_erc20_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1714 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_slashing_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_slashing_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     8266 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_stake_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/dpos_stake_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1929 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/ethereum_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/ethereum_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     5968 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/multi_sign_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/multi_sign_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     7210 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/private_compute_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/private_compute_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1460 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/pubkey_manage_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/pubkey_manage_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)    25107 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/relay_cross_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/relay_cross_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3326 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/store_hot_cold_data_separate_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/store_hot_cold_data_separate_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2092 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/store_snapshot_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/store_snapshot_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3855 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/subscribe_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/subscribe_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2465 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/system_contract_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/system_contract_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1413 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/test_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/test_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1390 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/transaction_manager_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/syscontract/transaction_manager_pb2_grpc.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.408241 chainmaker-3.0.0/chainmaker/protos/txpool/
+-rw-r--r--   0 superhin   (502) staff       (20)    13577 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/txpool/transaction_pool_pb2.py
+-rw-r--r--   0 superhin   (502) staff       (20)      159 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/protos/txpool/transaction_pool_pb2_grpc.py
+-rw-r--r--   0 superhin   (502) staff       (20)    19774 2023-08-01 07:12:15.000000 chainmaker-3.0.0/chainmaker/sdk_config.py
+-rw-r--r--   0 superhin   (502) staff       (20)      184 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/user.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.423241 chainmaker-3.0.0/chainmaker/utils/
+-rw-r--r--   0 superhin   (502) staff       (20)       30 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/utils/__init__.py
+-rw-r--r--   0 superhin   (502) staff       (20)    10772 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/address_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)    14053 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/utils/archive_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)     5710 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/asn1_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)    40094 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/utils/cmc_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)     5676 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/utils/common.py
+-rw-r--r--   0 superhin   (502) staff       (20)    16787 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/contract_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)    26710 2023-08-01 08:15:44.000000 chainmaker-3.0.0/chainmaker/utils/crypto_config_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)    12746 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/crypto_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)    29098 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/deploy_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3819 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/evm_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)     4745 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/file_utils.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.429298 chainmaker-3.0.0/chainmaker/utils/gm/
+-rw-r--r--   0 superhin   (502) staff       (20)        0 2022-09-26 09:13:08.000000 chainmaker-3.0.0/chainmaker/utils/gm/__init__.py
+-rw-r--r--   0 superhin   (502) staff       (20)     5397 2022-12-20 03:35:04.000000 chainmaker-3.0.0/chainmaker/utils/gm/ec.py
+-rw-r--r--   0 superhin   (502) staff       (20)      949 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/utils/gm/func.py
+-rw-r--r--   0 superhin   (502) staff       (20)    16778 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/utils/gm/sm2.py
+-rw-r--r--   0 superhin   (502) staff       (20)     5224 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/utils/gm/sm3.py
+-rw-r--r--   0 superhin   (502) staff       (20)     7197 2023-06-14 06:15:05.000000 chainmaker-3.0.0/chainmaker/utils/gm/sm4.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1324 2022-12-20 03:35:04.000000 chainmaker-3.0.0/chainmaker/utils/log_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)     9893 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/result_utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)    83233 2023-08-01 07:10:59.000000 chainmaker-3.0.0/chainmaker/utils/server_utils.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-08-01 08:18:06.325077 chainmaker-3.0.0/chainmaker.egg-info/
+-rw-r--r--   0 superhin   (502) staff       (20)      303 2023-08-01 08:18:06.000000 chainmaker-3.0.0/chainmaker.egg-info/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)     6437 2023-08-01 08:18:06.000000 chainmaker-3.0.0/chainmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-08-01 08:18:06.000000 chainmaker-3.0.0/chainmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       86 2023-08-01 08:18:06.000000 chainmaker-3.0.0/chainmaker.egg-info/requires.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       11 2023-08-01 08:18:06.000000 chainmaker-3.0.0/chainmaker.egg-info/top_level.txt
+-rw-r--r--   0 superhin   (502) staff       (20)      103 2021-09-15 06:14:28.000000 chainmaker-3.0.0/pyproject.toml
+-rw-r--r--   0 superhin   (502) staff       (20)       38 2023-08-01 08:18:06.430890 chainmaker-3.0.0/setup.cfg
+-rw-r--r--   0 superhin   (502) staff       (20)     1396 2023-08-01 07:10:59.000000 chainmaker-3.0.0/setup.py
```

### Comparing `chainmaker-2.3.2/LICENSE` & `chainmaker-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainmaker-2.3.2/README.md` & `chainmaker-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `chainmaker-2.3.2/chainmaker/chain_client.py` & `chainmaker-3.0.0/chainmaker/chain_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,37 +11,38 @@
 from pathlib import Path
 from typing import Union, List
 
 import grpc
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
 
 from chainmaker import exceptions
-from chainmaker.apis import (ChainConfigMixIn, ChainQueryMixIn, ArchiveMixIn,
-                             CertManageMixIn, ChainMakerServerMixIn,
-                             DPosErc20MixIn, DPosStakeMixIn,
+from chainmaker.apis import (ChainConfigMixIn, ChainQueryMixIn, ArchiveMixIn, CanonicalTxResultMixIn,
+                             CertManageMixIn, ChainMakerServerMixIn, ConsensusMixIn,
+                             DPosErc20MixIn, DPosStakeMixIn, DPosSlashingMixIn,
                              AccountManagerMixIn, MultiSignMixin, PubkeyManageMixIn,
-                             SubscribeManageMixIn, SystemContractMixIn, ContractQueryMixIn,
+                             SubscribeManageMixIn, SystemContractMixIn, ContractQueryMixIn, TxPoolMixIn,
                              UserContractMixIn, AccountManagerWithEndorsers, CertManageWithEndorsers,
                              ArchiveWithEndorsers, ContractManageWithEndorsers, ChainConfigWithEndorsers,
-                             PubkeyManageWithEndorsers, DPosErc20WithEndorsers, DPosStakeWithEndorsers)
+                             PubkeyManageWithEndorsers, DPosErc20WithEndorsers, DPosStakeWithEndorsers,
+                             DPosSlashingWithEndorsers, DPosDistributionWithEndorsers, DPosDistributionMixIn)
+from chainmaker.apis.chain_query import ChainQueryExtras
 from chainmaker.apis.private_compute import PrivateComputeMixIn
 from chainmaker.client_node import ClientNode
 from chainmaker.client_user import ClientUser
 from chainmaker.conn_pool import ConnectionPool
 from chainmaker.exceptions import GetTxTimeoutError
 from chainmaker.keys import (AuthType, HashType, MemberType, AddrType, Certificate, PublicKey, PrivateKey,
                              ConsensusType)
 from chainmaker.payload import PayloadBuilder
 from chainmaker.protos import (RpcNodeStub, Payload, TxRequest, EndorsementEntry, TxType, TxResponse, TxStatusCode,
                                Result)
 from chainmaker.protos.config.chain_config_pb2 import ChainConfig
 from chainmaker.sdk_config import (DefaultConfig, SdkConfig,
                                    ChainClientConfig, DEFAULT_ARCHIVE_CONFIG, DEFAULT_PKCS11_CONFIG,
                                    DEFAULT_RPC_CLIENT_CONFIG, Pkcs11Config)
-from chainmaker.user import User
 from chainmaker.utils.common import ensure_enum
 from chainmaker.utils.log_utils import get_logger
 
 SDK_CONFIG_USER_CONFIG_FILTER = {"user_sign_key_file_path", "user_sign_crt_file_path", "user_sign_key_pwd",
                                  "user_key_file_path", "user_crt_file_path", "user_key_pwd",
                                  "user_enc_key_file_path", "user_enc_crt_file_path", "user_enc_key_pwd",
                                  "org_id", "crypto", "auth_type", "alias"}
@@ -49,15 +50,16 @@
 SDK_LOGGER = get_logger(DefaultConfig.logger_name, DefaultConfig.log_level, format=DefaultConfig.log_format,
                         datefmt=DefaultConfig.log_datefmt, log_file=DefaultConfig.log_file)
 
 
 class ChainClient(SystemContractMixIn, ChainQueryMixIn, UserContractMixIn, ContractQueryMixIn, ChainConfigMixIn,
                   CertManageMixIn,
                   SubscribeManageMixIn, ArchiveMixIn, PubkeyManageMixIn, AccountManagerMixIn,
-                  MultiSignMixin, ChainMakerServerMixIn, DPosErc20MixIn, DPosStakeMixIn,
+                  MultiSignMixin, ChainMakerServerMixIn, TxPoolMixIn, CanonicalTxResultMixIn,
+                  ConsensusMixIn, DPosErc20MixIn, DPosStakeMixIn, DPosSlashingMixIn, DPosDistributionMixIn,
                   PrivateComputeMixIn):
 
     def __init__(self, chain_id, user: ClientUser, nodes: List[ClientNode], conn_node: int = None,
                  node_index: int = None):
         self._chain_id = chain_id
         self.user = user  # todo change to _user
         self.nodes = nodes  # todo change to _nodes
@@ -314,32 +316,26 @@
         """
         签名Payload二进制内容
         :param payload_bytes: Payload二进制内容
         :return: 背书条目
         """
         return self.user.sign(payload_bytes)
 
-    def _generate_tx_request(self, payload: Payload, endorsers: List[EndorsementEntry] = None,
-                             payer: User = None) -> TxRequest:
+    def _generate_tx_request(self, payload: Payload, endorsers: List[EndorsementEntry] = None) -> TxRequest:
         payload_bytes = payload.SerializeToString()
         sender = self.sign(payload_bytes)
-        if payer is None:
-            payer = sender
-        else:
-            payer = payer.sign(payload_bytes)
         tx_request = TxRequest(
             payload=payload,
             sender=sender,
-            endorsers=endorsers,
-            payer=payer,
+            endorsers=endorsers
         )
         # self.logger.debug('[Sdk] Generate txRequest: %s', json_format.MessageToJson(tx_request))
         return tx_request
 
-    def _send_request(self, payload: Payload, endorsers: List[EndorsementEntry] = None, payer: User = None,
+    def _send_request(self, payload: Payload, endorsers: List[EndorsementEntry] = None,
                       timeout: int = None) -> TxResponse:
         """
         发送带超时时间的交易请求
         :param payload: 待签名请求Payload
         :param endorsers: 背书列表
         :param timeout: 超时时间
         :return: 交易响应TxResponse对象
@@ -354,45 +350,43 @@
                     else DefaultConfig.rpc_send_tx_timeout
 
         # 处理默认背书
         if self.endorsers:
             endorsers = endorsers or self._create_endorsers(payload, endorsers)
 
         # 构造请求结构
-        tx_request = self._generate_tx_request(payload, endorsers, payer)
+        tx_request = self._generate_tx_request(payload, endorsers)
 
         # 仅记录Invoke交易
         if self._enabled_tx_records and tx_request.payload.tx_type == TxType.INVOKE_CONTRACT:
             self._tx_records.append(tx_request)
 
         return self._pool.send_rpc_request(tx_request, timeout=timeout, conn_node=self._conn_node)
 
     def _send_request_with_timeout(self, payload: Payload, endorsers: List[EndorsementEntry] = None,
-                                   payer: User = None,
                                    timeout: int = None) -> TxResponse:
         warnings.warn('[Sdk] please use cc._send_request instead', DeprecationWarning)
-        return self._send_request(payload, endorsers, payer, timeout)
+        return self._send_request(payload, endorsers, timeout)
 
     @staticmethod
     def _handle_errors(tx_response):
         if tx_response.code != TxStatusCode.SUCCESS:
             if tx_response.code == 5:  # InternalError
                 exceptions.handle_internal_error(tx_response)
             elif tx_response.code == 4:  # ContractFail
                 exceptions.handle_contract_fail(tx_response)
             err_class = exceptions.TX_RESPONSE_ERROR_MAP.get(tx_response.code)
             raise err_class(TxStatusCode.Name(tx_response.code), tx_response.message)
         return tx_response
 
-    def send_request(self, payload: Payload, endorsers: List[EndorsementEntry] = None, payer: User = None,
+    def send_request(self, payload: Payload, endorsers: List[EndorsementEntry] = None,
                      timeout: int = None) -> TxResponse:
         """
         发送交易请求并检查是否成功
         带重连机制，基于 self._send_request_with_retry_connect
-        :param payer:
         :param payload: 待签名请求Payload
         :param endorsers: 背书列表
         :param timeout: 超时时间
         :return: 交易响应TxResponse对象
         :raise 重连超过retry_limit限制仍无法成功时抛出 RpcConnectError
         :raise: RequestError错误子类，如InvalidParameter等
         """
@@ -400,15 +394,15 @@
         # handle txpool is full error
         retry_timeout = DefaultConfig.txpool_full_retry_timeout
         retry_interval = DefaultConfig.txpool_full_retry_interval
         start = time.time()
         while (tx_response.code == 5 and 'TxPool is full' in tx_response.message) and (
                 time.time() - start < retry_timeout):
             time.sleep(retry_interval)
-            tx_response = self._send_request(payload, endorsers, payer, timeout)
+            tx_response = self._send_request(payload, endorsers, timeout)
         return self._handle_errors(tx_response)
 
     @staticmethod
     def _update_tx_response_with_result(tx_response: TxResponse, result: Result) -> TxResponse:
         """
         更新交易响应，将轮询得到的交易结果中的信息添加到交易响应中
         :param tx_response: 原交易响应
@@ -424,31 +418,29 @@
         tx_response.contract_result.gas_used = result.contract_result.gas_used
         for contract_event in result.contract_result.contract_event:
             tx_response.contract_result.contract_event.append(contract_event)
 
         return tx_response
 
     def send_request_with_sync_result(self, payload: Payload, endorsers: List[EndorsementEntry] = None,
-                                      payer: User = None,
                                       timeout: int = None, with_sync_result: bool = None) -> TxResponse:
         """
         发送请求并支持轮询交易结果
-        :param payer:
         :param payload: 待签名请求Payload
         :param timeout: 超时时间
         :param with_sync_result: 是否同步获取交易结果，默认为False
         :param endorsers: 背书配置
         :return: 交易响应TxResponse对象
         :raise: RequestError错误子类，如InvalidParameter等
         :raise: 在指定时间（self.check_tx_timeout）内未获取到结果抛出，GetTxTimeoutError
         """
         if with_sync_result is None:
             with_sync_result = self._with_sync_result
 
-        tx_response = self.send_request(payload, endorsers, payer, timeout)
+        tx_response = self.send_request(payload, endorsers, timeout)
 
         if with_sync_result is True:
             tx_response.tx_id = payload.tx_id
             result = self.get_sync_result(payload.tx_id)
             tx_response = self._update_tx_response_with_result(tx_response, result)
 
         return tx_response
@@ -599,52 +591,50 @@
         return self.user.sign_cert_bytes
 
     def get_local_cert_alias(self):
         """获取用户证书别名 同 self.alias"""
         warnings.warn('[Sdk] please use cc.alias instead', DeprecationWarning)
         return self.user.alias
 
-    def send_manage_request(self, payload: Payload, endorse_users: List[ClientUser] = None, payer: User = None,
+    def send_manage_request(self, payload: Payload, endorse_users: List[ClientUser] = None,
                             timeout: int = None, with_sync_result: bool = True) -> TxResponse:
         """
         发送带默认背书的管理请求
-        :param payer:
         :param payload: 待签名请求Payload
         :param endorse_users: 背书用户列表，默认为None并使用self.endorse_users
         :param timeout: 超时时间
         :param with_sync_result: 是否同步交易结果，默认为True
         :return: 交易响应TxResponse
         """
         # warnings.warn('[Sdk] please use ChainManager instead for client with default endorsers', DeprecationWarning)
         self._debug('begin to send manage request with default endorsers [tx_id:%s]' % payload.tx_id)
         if endorse_users is None:
             endorse_users = self.endorsers  # 背书用户
 
         endorsers = self._create_endorsers(payload, endorse_users)
 
-        response = self.send_request_with_sync_result(payload, endorsers, payer, timeout, with_sync_result)
+        response = self.send_request_with_sync_result(payload, endorsers, timeout, with_sync_result)
         return response
 
     def _send_request_with_retry_connect(self, payload: Payload, endorsers: List[EndorsementEntry] = None,
-                                         payer: User = None,
                                          timeout: int = None) -> TxResponse:
         """
         发送带重连的交易请求
         基于self._send_request_with_timeout
         :param payload: 待签名请求Payload
         :param endorsers: 背书列表
         :param timeout: 超时时间
         :return: 交易响应TxResponse对象
         :raise 重连超过retry_limit限制仍无法成功时抛出 RpcConnectError
         """
         warnings.warn('[Sdk] has moved to conn_poll, use cc._send_request() instead', DeprecationWarning)
         err_msg = ''
         for i in range(DefaultConfig.rpc_retry_limit):
             try:
-                return self._send_request(payload, endorsers, payer, timeout)
+                return self._send_request(payload, endorsers, timeout)
             except grpc._channel._InactiveRpcError as ex:
                 err_msg = exceptions.ERR_MSG_MAP.get(ex.details(), ex.details())
                 time.sleep(DefaultConfig.rpc_retry_interval // 1000)  # 毫秒
         else:
             self._logger.error("[Sdk] statusErr.Code() : %s")
 
             raise exceptions.RpcConnectError(
@@ -689,15 +679,15 @@
     #     self.user.sign_key_bytes = sign_key_bytes
     #     self.user.sign_cert_bytes = sign_cert_bytes
 
 
 class ChainClientWithEndorsers(ChainClient, AccountManagerWithEndorsers, CertManageWithEndorsers,
                                ChainConfigWithEndorsers, ContractManageWithEndorsers, PubkeyManageWithEndorsers,
                                ArchiveWithEndorsers, DPosErc20WithEndorsers, DPosStakeWithEndorsers,
-                               ):
+                               DPosSlashingWithEndorsers, DPosDistributionWithEndorsers, ChainQueryExtras):
     @property
     def chain_config(self) -> ChainConfig:
         """链配置(缓存)"""
         if not hasattr(self, '_cached_chain_config') or getattr(self, '_cached_chain_config') is None:
             setattr(self, '_cached_chain_config', self.get_chain_config())
         return getattr(self, '_cached_chain_config')
```

### Comparing `chainmaker-2.3.2/chainmaker/chain_manager.py` & `chainmaker-3.0.0/chainmaker/chain_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 import uuid
 from pathlib import Path
 from typing import List, Union, Dict, Callable, Any
 
 from hostz import Host
 
 from chainmaker.chain_client import ChainClientWithEndorsers
+from chainmaker.client_user import ClientUser
 from chainmaker.keys import (ChainConfigMethod, ParamKey, Role, AddrType, RuntimeType,
                              ContractManageMethod, SystemContractName, ResourceName, Rule, RechargeGasItem,
-                             ContractStatus)
+                             ContractStatus, TxType, TxStage)
 from chainmaker.protos import (Payload, TxResponse, BlockHeader, BlockInfo, Contract, CertInfos, Result,
                                TransactionInfo, ChainConfig,
-                               ResourcePolicy, MultiSignInfo, ChainList, ChainInfo, BlockWithRWSet,
-                               AliasInfos)
+                               ResourcePolicy, MultiSignInfo, ChainList, ChainInfo, BlockWithRWSet, ValidatorVector,
+                               Delegation, DelegationInfo, Epoch, AliasInfos, Transaction, TxPoolStatus)
 from chainmaker.sdk_config import DefaultConfig
-from chainmaker.user import User
 from chainmaker.utils import (file_utils, crypto_utils, crypto_config_utils, result_utils, address_utils, common,
                               server_utils, cmc_utils)
 from chainmaker.utils.common import ensure_enum
 from chainmaker.utils.file_utils import load_byte_code
 
 
 def with_user_endorsers(method):
@@ -39,19 +39,15 @@
         user = kwargs.pop('user') if 'user' in kwargs else None
         endorsers = kwargs.pop('endorsers') if 'endorsers' in kwargs else None
         endorsers_cnt = kwargs.pop('endorsers_cnt') if 'endorsers_cnt' in kwargs else None
         conn_node = kwargs.pop('conn_node') if 'conn_node' in kwargs else None
         alias = kwargs.pop('alias') if 'alias' in kwargs else None
         enable_cert_hash = kwargs.pop('enable_cert_hash') if 'enable_cert_hash' in kwargs else None
 
-        if 'payer' in kwargs:
-            payer = kwargs.pop('payer')
-            kwargs['payer'] = self._crypto_config.get_user(payer)
-
-        if user or endorsers or endorsers_cnt:
+        if user:
             chain_id = self._cc.chain_id
             cc = self._crypto_config.new_chain_client(user, endorsers=endorsers, endorsers_cnt=endorsers_cnt,
                                                       conn_node=conn_node, alias=alias,
                                                       enable_cert_hash=enable_cert_hash, chain_id=chain_id)
             if hasattr(self, '_logger'):
                 setattr(cc, '_logger', getattr(self, '_logger'))
 
@@ -1172,19 +1168,19 @@
         :raise: RequestError: 请求出错
         :raise: AssertionError: 响应code不为0,检查响应时抛出断言失败
         :raise: 当数据不是JSON格式时，抛出json.decoder.JSONDecodeError
         """
         self._info("获取全部合约列表")
         return self._cc.get_all_contracts()
 
-    # 01-17 通过交易Id获取Merkle树路径
+    # 01-17 查询交易存在性证明
     @with_user_endorsers
-    def get_merkle_path_by_tx_id(self, tx_id: str) -> bytes:
+    def get_merkle_path_by_tx_id(self, tx_id: str) -> bool:
         """
-        通过交易Id获取Merkle树路径
+        查询交易存在性证明
         <01-17-CHAIN_QUERY-GET_MERKLE_PATH_BY_TX_ID>
         :param tx_id: 交易Id
         :return: Merkle树路径
         """
         self._info(f"通过交易Id {tx_id} 获取Merkle树路径")
         return self._cc.get_merkle_path_by_tx_id(tx_id)
 
@@ -1562,49 +1558,45 @@
 
 # 04
 class MultiSignOps(BaseOps):
     """多签管理"""
 
     # 04-00 发起多签请求
     @with_user_endorsers
-    def req(self, params: Union[list, dict], tx_id: str = None, gas_limit: int = None, payer: User = None,
-            timeout: int = None,
+    def req(self, params: Union[list, dict], tx_id: str = None, timeout: int = None,
             with_sync_result: bool = None) -> TxResponse:
         """
         发起多签请求
         <04-00-MULTI_SIGN-REQ>
-        :param payer:
-        :param gas_limit:
         :param params: 多签请求参数
         :param tx_id: 指定交易Id
         :param timeout: 请求超时时间
         :param with_sync_result: 是否同步获取交易结果
         :return: 交易响应或交易信息
         """
         self._info(f"发起多签请求 {params}")
-        payload = self._cc.create_multi_sign_req_payload(params, tx_id, gas_limit=gas_limit)
-        tx_response = self._cc.multi_sign_req(payload, payer=payer, timeout=timeout, with_sync_result=with_sync_result)
+        payload = self._cc.create_multi_sign_req_payload(params, tx_id)
+        tx_response = self._cc.multi_sign_req(payload, timeout=timeout, with_sync_result=with_sync_result)
         return tx_response
 
     # 04-01 对多签请求Payload进行投票
     @with_user_endorsers
-    def vote(self, tx_id: str, is_agree: bool = True, endorser: User = None, gas_limit: int = None, payer: User = None,
+    def vote(self, tx_id: str, is_agree: bool = True, endorser: ClientUser = None,
              timeout: int = None, with_sync_result: bool = None) -> TxResponse:
         """
         根据交易Id对多签请求进行投票
-        :param gas_limit:
         :param tx_id: 交易Id
         :param endorser: 投票用户对象
         :param is_agree: 是否同意，true为同意，false则反对
         :param timeout: 请求超时时间
         :param with_sync_result: 是否同步获取交易结果
         :return: 交易响应或交易信息
         """
         self._info(f"对多签请求 {tx_id} 进行投票")
-        return self._cc.multi_sign_vote_by_tx_id(tx_id, endorser, is_agree, gas_limit, payer, timeout, with_sync_result)
+        return self._cc.multi_sign_vote_by_tx_id(tx_id, endorser, is_agree, timeout, with_sync_result)
 
     # 04-02 查询多签状态
     @with_user_endorsers
     def query(self, tx_id: str, timeout: int = None) -> MultiSignInfo:
         """
         查询多签状态
         <04-02-MULTI_SIGN-QUERY>
@@ -1612,45 +1604,42 @@
         :param timeout: RPC请求超时时间
         :return: 多签信息
         """
         self._info(f"查询交易 {tx_id} 多签状态 ")
         return self._cc.multi_sign_query(tx_id, timeout=timeout)
 
     @with_user_endorsers
-    def trig(self, tx_id: str, gas_limit: int = None, payer: User = None, timeout: int = None,
-             with_sync_result: bool = None) -> TxResponse:
+    def trig(self, tx_id: str, gas_limit: int = None, timeout: int = None, with_sync_result: bool = None) -> TxResponse:
         """
         发送线上多签触发请求到节点 v2.3.1新增
-        :param payer:
         :param gas_limit:
         :param tx_id: 多签请求交易Id
         :param timeout: RPC请求超时时间
         :param with_sync_result: 是否同步轮询交易结果
         :return: 交易相应
         """
         self._info("触发多签执行")
         # tx = self._cc.get_tx_by_tx_id(tx_id)
         # multi_sign_req_payload = tx.transaction.payload
-        return self._cc.multi_sign_trig(tx_id=tx_id, gas_limit=gas_limit, payer=payer,
+        return self._cc.multi_sign_trig(tx_id=tx_id, gas_limit=gas_limit,
                                         timeout=timeout, with_sync_result=with_sync_result)
 
     @with_user_endorsers
     def create_contract_req(self, contract_name: str, byte_code_path: Union[Path, str],
-                            runtime_type: Union[RuntimeType, str], version: str = '1.0', gas_limit: int = None,
-                            payer: User = None) -> TxResponse:
+                            runtime_type: Union[RuntimeType, str], version: str = '1.0') -> TxResponse:
         byte_code = load_byte_code(byte_code_path)
         runtime_type = ensure_enum(runtime_type, RuntimeType).name
         params = {'SYS_CONTRACT_NAME': 'CONTRACT_MANAGE',
                   'SYS_METHOD': 'INIT_CONTRACT',
                   'CONTRACT_NAME': contract_name,
                   'CONTRACT_VERSION': version,
                   'CONTRACT_BYTECODE': byte_code,
                   'CONTRACT_RUNTIME_TYPE': runtime_type
                   }
-        return self.req(params, gas_limit=gas_limit, payer=payer)
+        return self.req(params)
 
 
 # 05
 class ContractManageOps(BaseOps):
     # ================================ 合约管理 ===============================================
     # 05-00 获取合约信息
     @with_user_endorsers
@@ -1755,19 +1744,17 @@
         contract = self._cc.get_contract_info(contract_name)
         return contract is not None
 
     # 05-00 创建合约
     @with_user_endorsers
     def create_contract(self, contract_name: str, byte_code_path: str, runtime_type: Union[RuntimeType, str],
                         params: dict = None, version: str = None, gas_limit: int = None, tx_id: str = None,
-                        payer: User = None,
                         timeout: int = None, with_sync_result: bool = None) -> TxResponse:
         """
         创建合约
-        :param payer:
         :param contract_name: 合约名
         :param version: 合约版本
         :param byte_code_path: 合约字节码：可以是字节码；合约文件路径；或者 hex编码字符串；或者 base64编码字符串。
         :param runtime_type: contract_pb2.RuntimeType.WASMER
         :param params: 合约参数，dict类型，key 和 value 尽量为字符串
         :param gas_limit: Gas限制
         :param tx_id: 指定交易Id
@@ -1775,24 +1762,25 @@
         :param with_sync_result: 是否同步轮询交易结果
         :return: 交易响应
         :raises ValueError: 如果 byte_code 不能转成合约字节码
         :raises: RequestError: 请求失败
         """
         # runtime_type = ensure_enum(runtime_type, RuntimeType)
         self._info(f'创建{runtime_type}合约 {contract_name}')
-        return self._cc.create_contract(contract_name, byte_code_path, runtime_type, params, version,
-                                        gas_limit, tx_id, payer, timeout, with_sync_result)
+        payload = self._cc.create_contract_create_payload(contract_name, version, byte_code_path, runtime_type,
+                                                          params, gas_limit, tx_id)
+
+        return self._cc.send_manage_request(payload, timeout=timeout, with_sync_result=with_sync_result)
 
     @with_user_endorsers
     def invoke_contract(self, contract_name: str, method: str, params: dict = None,
-                        gas_limit: int = None, payer: User = None, tx_id: str = None, result_type: str = None,
+                        gas_limit: int = None, tx_id: str = None, result_type: str = None,
                         timeout: int = None, with_sync_result: bool = None) -> TxResponse:
         """
         调用合约
-        :param payer:
         :param contract_name: 合约名
         :param method: 合约方法名
         :param params: 合约方法参数
         :param gas_limit: 交易Gas限制
         :param tx_id: 指定交易Id
         :param result_type: 结果类型, 用于解析响应中的result
         :param timeout: RPC请求超时时间
@@ -1800,16 +1788,15 @@
         :return: TxResponse
         :raises RequestError: 请求失败
         """
         if params:
             self._info(f'调用合约 {contract_name} method: {method} params: {params}')
         else:
             self._info(f'调用合约 {contract_name} method: {method}')
-        response = self._cc.invoke_contract(contract_name, method, params, tx_id, gas_limit, payer, timeout,
-                                            with_sync_result)
+        response = self._cc.invoke_contract(contract_name, method, params, tx_id, gas_limit, timeout, with_sync_result)
         return response if result_type is None else result_utils.parse_result(response, result_type)
 
     @with_user_endorsers
     def query_contract(self, contract_name: str, method: str, params: Union[dict, list] = None, result_type: str = None,
                        timeout: int = None) -> TxResponse:
         """
         查询用户合约
@@ -1828,15 +1815,14 @@
         response = self._cc.query_contract(contract_name, method, params, timeout=timeout)
         return response if result_type is None else result_utils.parse_result(response, result_type)
 
     # 05-01 升级合约
     @with_user_endorsers
     def upgrade_contract(self, contract_name: str, byte_code_path: str, runtime_type: Union[RuntimeType, str],
                          params: dict = None, version: str = None, gas_limit: int = None, tx_id: str = None,
-                         payer: User = None,
                          timeout: int = None, with_sync_result: bool = None) -> TxResponse:
         """
         升级合约
         :param contract_name: 合约名
         :param version: 合约版本
         :param byte_code_path: 合约字节码：可以是字节码；合约文件路径；或者 hex编码字符串；或者 base64编码字符串。
         :param runtime_type: contract_pb2.RuntimeType.WASMER
@@ -1848,16 +1834,18 @@
         :return: 交易响应
         :raises ValueError: 如果 byte_code 不能转成合约字节码
         :raises: RequestError: 请求失败
         """
         if version is None:
             version = self.gen_new_contract_version(contract_name)
         self._info(f'升级{runtime_type}合约 {contract_name} version: {version}')
-        return self._cc.upgrade_contract(contract_name, byte_code_path, runtime_type, params, version,
-                                         gas_limit, tx_id, payer, timeout, with_sync_result)
+        payload = self._cc.create_contract_upgrade_payload(contract_name, version, byte_code_path, runtime_type,
+                                                           params, gas_limit, tx_id)
+
+        return self._cc.send_manage_request(payload, timeout=timeout, with_sync_result=with_sync_result)
 
     # 05-02 冻结合约
     @with_user_endorsers
     def freeze_contract(self, contract_name: str, tx_id: str = None, timeout: int = None,
                         with_sync_result: bool = None) -> TxResponse:
         """
         冻结合约
@@ -1865,15 +1853,17 @@
         :param tx_id: 指定交易Id
         :param timeout: RPC请求超时时间
         :param with_sync_result: 是否同步轮询交易结果
         :return: 交易响应
         :raises: RequestError: 请求失败
         """
         self._info(f'冻结合约 {contract_name}')
-        payload = self._cc.freeze_contract(contract_name, tx_id, timeout, with_sync_result)
+        payload = self._cc._create_contract_manage_payload(ContractManageMethod.FREEZE_CONTRACT.name, contract_name,
+                                                           tx_id=tx_id)
+        return self._cc.send_manage_request(payload, timeout=timeout, with_sync_result=with_sync_result)
 
     # 05-03 解冻合约
     @with_user_endorsers
     def unfreeze_contract(self, contract_name: str, tx_id: str = None, timeout: int = None,
                           with_sync_result: bool = None) -> TxResponse:
         """
         解冻合约
@@ -1881,15 +1871,17 @@
         :param tx_id: 指定交易Id
         :param timeout: RPC请求超时时间
         :param with_sync_result: 是否同步轮询交易结果
         :return: 交易响应
         :raises: RequestError: 请求失败
         """
         self._info(f'解冻合约 {contract_name}')
-        payload = self._cc.unfreeze_contract(contract_name, tx_id, timeout, with_sync_result)
+        payload = self._cc._create_contract_manage_payload(ContractManageMethod.UNFREEZE_CONTRACT.name, contract_name,
+                                                           tx_id=tx_id)
+        return self._cc.send_manage_request(payload, timeout=timeout, with_sync_result=with_sync_result)
 
     # 05-04 吊销合约
     @with_user_endorsers
     def revoke_contract(self, contract_name: str, tx_id=None, timeout: int = None,
                         with_sync_result: bool = None) -> TxResponse:
         """
         吊销合约
@@ -1897,15 +1889,17 @@
         :param tx_id: 指定交易Id
         :param timeout: RPC请求超时时间
         :param with_sync_result: 是否同步轮询交易结果
         :return: 交易响应
         :raises: RequestError: 请求失败
         """
         self._info(f'吊销合约 {contract_name}')
-        payload = self._cc.revoke_contract(contract_name, tx_id, timeout, with_sync_result)
+        payload = self._cc._create_contract_manage_payload(ContractManageMethod.REVOKE_CONTRACT.name, contract_name,
+                                                           tx_id=tx_id)
+        return self._cc.send_manage_request(payload, timeout=timeout, with_sync_result=with_sync_result)
 
     def gen_new_contract_version(self, contract_name: str, increase: float = 1.0) -> str:
         """
         查询合约当前版本，并生成合约新版本号
         :param contract_name: 合约名称
         :param increase: 在原版本基础上增加值，默认原版本+1
         :return: 合约版本
@@ -2221,14 +2215,110 @@
         return self._cc.total()
 
 
 # 08 DPOS共识权益操作
 class DposStakeOps(BaseOps):
     """DPOS共识权益操作"""
 
+    # 08-00 查询所有的候选人
+    @with_user_endorsers
+    def get_all_candidates(self) -> ValidatorVector:
+        """
+        查询所有的候选人
+        <08-00-DPOS_STAKE-GET_ALL_CANDIDATES>
+        :return: 候选人列表
+        """
+        self._info('查询所有的候选人')
+        return self._cc.get_all_candidates()
+
+    # 08-01 通过地址获取验证人的信息
+    @with_user_endorsers
+    def get_validator_by_address(self, address: str):
+        """
+        通过地址获取验证人的信息
+        <08-01-DPOS_STAKE-GET_VALIDATOR_BY_ADDRESS>
+        :param address:
+        :return:
+        """
+        self._info(f'通过地址 {address} 获取验证人的信息')
+        return self._cc.get_validator_by_address(address)
+
+    # 08-02 抵押权益到验证人
+    @with_user_endorsers
+    def delegate(self, address: str, amount: int) -> Delegation:  # todo 确认是否需要轮训
+        """
+        抵押权益到验证人
+        <08-02-DPOS_STAKE-DELEGATE>
+        :param address:
+        :param amount:
+        :return:
+        """
+        self._info(f'抵押权益到验证人 address: {address} amount: {amount}')
+        return self._cc.delegate(address, amount)
+
+    # 08-03 查询指定地址的抵押信息
+    @with_user_endorsers
+    def get_delegations_by_address(self, address: str) -> DelegationInfo:
+        """
+        查询指定地址的抵押信息
+        <08-03-DPOS_STAKE-GET_DELEGATIONS_BY_ADDRESS>
+        :param address:
+        :return:
+        """
+        self._info(f'查询指定地址 {address} 的抵押信息')
+        return self._cc.get_delegations_by_address(address)
+
+    # 08-04 查询指定地址的抵押信息
+    @with_user_endorsers
+    def get_user_delegation_by_validator(self, delegator: str, validator: str) -> Delegation:
+        """
+        查询指定地址的抵押信息
+        <08-04-DPOS_STAKE-GET_USER_DELEGATION_BY_VALIDATOR>
+        :param delegator:
+        :param validator:
+        :return:
+        """
+        self._info(f'查询指定地址的抵押信息 delegator: {delegator} validator: {validator}')
+        return self._cc.get_user_delegation_by_validator(delegator, validator)
+
+    # 08-04 从验证人解除抵押的权益
+    @with_user_endorsers
+    def undelegate(self, address: str, amount: int) -> Delegation:
+        """
+        从验证人解除抵押的权益
+        <08-05-DPOS_STAKE-UNDELEGATE>
+        :param address:
+        :param amount:
+        :return:
+        """
+        self._info(f'从验证人解除抵押的权益 address: {address} amount: {amount}')
+        return self._cc.undelegate(address, amount)
+
+    # 08-06 查询指定世代信息
+    @with_user_endorsers
+    def get_epoch_by_id(self, epoch_id: str) -> Epoch:
+        """
+        查询指定世代信息
+        <08-06-DPOS_STAKE-READ_EPOCH_BY_ID>
+        :param epoch_id:
+        :return:
+        """
+        self._info(f'查询世代 {epoch_id} 信息')
+        return self._cc.get_epoch_by_id(epoch_id)
+
+    # 08-07 查询当前世代信息
+    @with_user_endorsers
+    def get_last_epoch(self) -> Epoch:
+        """
+        查询当前世代信息
+        <08-07-DPOS_STAKE-READ_LATEST_EPOCH>
+        :return:
+        """
+        return self._cc.get_last_epoch()
+
     # 08-08 Stake合约中设置验证人的NodeId
     @with_user_endorsers
     def set_node_id(self, node_id: str) -> str:
         """
         Stake合约中设置验证人的NodeId
         <08-08-DPOS_STAKE-SET_NODE_ID>
         :param node_id:
@@ -2702,14 +2792,232 @@
         :return:
         """
         self._info(f'Gas多账户收费')
         payload = self._cc.create_charge_gas_for_multi_account_payload(charge_gas_list)
         return self._cc.send_manage_request(payload, timeout=timeout, with_sync_result=with_sync_result)
 
 
+# 14 DPOS共识奖励操作
+class DposDistributionOps(BaseOps):
+    """DPOS共识奖励操作"""
+
+    # 14-00 奖励
+    def reward(self, timeout: int = None, with_sync_result: bool = None) -> TxResponse:  # todo
+        """
+        奖励
+        <14-00-DPOS_DISTRIBUTION-REWARD>
+        :param timeout: RPC请求超时时间
+        :param with_sync_result: 是否同步轮询交易结果
+        :return: 交易响应
+        """
+        raise NotImplementedError("待实现")
+
+    # 14-01 根据世代Id获取奖励
+    def get_distribution_by_epoch_id(self, epoch_id: str) -> dict:
+        """
+        <14-01-DPOS_DISTRIBUTION-GET_DISTRIBUTION_DETAIL>
+        :return:
+        """
+        return self._cc.get_distribution_by_epoch_id(epoch_id)
+
+    # 14-02 设置每个区块奖励数量
+    def set_distribution_per_block(self, distribution_per_block: int, timeout: int = None,
+                                   with_sync_result: bool = None) -> TxResponse:
+        """
+        设置每个区块奖励数量
+        <14-02-DPOS_DISTRIBUTION-SET_DISTRIBUTION_PER_BLOCK>
+        :param distribution_per_block:
+        :param timeout: RPC请求超时时间
+        :param with_sync_result: 是否同步轮询交易结果
+        :return: 交易响应
+        """
+        self._info("设置每个区块奖励数量为 %d" % distribution_per_block)
+        return self._cc.set_distribution_per_block(distribution_per_block, timeout, with_sync_result)
+
+    # 14-03 获取每个区块奖励数量
+    def get_distribution_per_block(self) -> int:
+        """
+        获取每个区块奖励数量
+        <14-03-DPOS_DISTRIBUTION-GET_DISTRIBUTION_PER_BLOCK>
+        :return:
+        """
+        self._info("获取每个区块奖励数量")
+        return self._cc.get_distribution_per_block()
+
+    # 14-04 设置从惩罚而来的奖励数量
+    def set_distribution_from_slashing(self, slashing_per_block: int, timeout: int = None,
+                                       with_sync_result: bool = None) -> TxResponse:
+        """
+        设置惩罚数量
+        <14-04-DPOS_DISTRIBUTION-SET_DISTRIBUTION_FROM_SLASHING>
+        :param slashing_per_block:
+        :param timeout: RPC请求超时时间
+        :param with_sync_result: 是否同步轮询交易结果
+        :return: 交易响应
+        """
+        raise NotImplementedError("待实现")
+
+    # 14-05 获取从惩罚而来的奖励数量
+    def get_distribution_from_slashing(self) -> str:
+        """
+        <14-05-DPOS_DISTRIBUTION-GET_DISTRIBUTION_FROM_SLASHING>
+        :return:
+        """
+        raise NotImplementedError("待实现")
+
+    # 14-06 设置Gas转换率
+    def set_gas_exchange_rate(self, gas_exchange_rate: int, timeout: int = None,
+                              with_sync_result: bool = None) -> TxResponse:
+        """
+        设置Gas转换率
+        <14-06-DPOS_DISTRIBUTION-SET_GAS_EXCHANGE_RATE>
+        :param gas_exchange_rate:
+        :param timeout: RPC请求超时时间
+        :param with_sync_result: 是否同步轮询交易结果
+        :return: 交易响应
+        """
+        self._info("设置Gas转换率为 %d" % gas_exchange_rate)
+        return self._cc.set_gas_exchange_rate(gas_exchange_rate, timeout, with_sync_result)
+
+    # 14-07 获取Gas转换率
+    def get_gas_exchange_rage(self) -> int:
+        """
+        <14-07-DPOS_DISTRIBUTION-SET_GAS_EXCHANGE_RATE>
+        :return:
+        """
+        self._info("获取Gas转换率")
+        return self._cc.get_gas_exchange_rage()
+
+
+# 15 DPOS共识惩罚操作
+class DposSlashingOps(BaseOps):
+    """DPOS共识惩罚操作"""
+
+    # 15-00 惩罚
+    def punish(self, timeout: int = None, with_sync_result: bool = None) -> TxResponse:  # todo 参数
+        """
+        惩罚
+        <15-00-DPOS_SLASHING-PUNISH>
+        :param timeout: RPC请求超时时间
+        :param with_sync_result: 是否同步轮询交易结果
+        :return: 交易响应
+        """
+        raise NotImplementedError("待实现")
+
+    # 15-02 设置区块惩罚数量
+    def set_slashing_per_block(self, slashing_per_block: int, timeout: int = None,
+                               with_sync_result: bool = None) -> TxResponse:
+        """
+        设置区块惩罚数量
+        <15-02-DPOS_SLASHING-SET_SLASHING_PER_BLOCK>
+         :param slashing_per_block:
+         :param timeout: RPC请求超时时间
+        :param with_sync_result: 是否同步轮询交易结果
+        :return: 交易响应
+        """
+        self._info("设置区块惩罚数量为 %d" % slashing_per_block)
+        return self._cc.set_slashing_per_block(slashing_per_block, timeout, with_sync_result)
+
+    # 15-03 获取区块惩罚数量
+    def get_slashing_per_block(self) -> int:
+        """
+        获取区块惩罚数量
+        <15-03-DPOS_SLASHING-GET_SLASHING_PER_BLOCK>
+        :return:
+        """
+        self._info("获取区块惩罚数量")
+        return self._cc.get_slashing_per_block()
+
+    # 15-04 查询惩罚账户余额
+    def get_slashing_balance(self) -> int:
+        """
+        查询惩罚账户余额
+        <15-04-DPOS_SLASHING-GET_SLASHING_ADDRESS_BALANCE>
+        :return:
+        """
+        self._info('查询惩罚账户余额')
+        return self._cc.get_slashing_balance()
+
+    # 15-05 通过世代Id获取惩罚数据
+    def get_slashing_by_epoch_id(self, epoch_id: str) -> dict:
+        """
+        通过世代Id获取惩罚数据
+        <15-05-DPOS_SLASHING-GET_SLASHING_DETAIL>
+        :return:
+        """
+        self._info('通过世代Id获取惩罚数据')
+        return self._cc.get_slashing_by_epoch_id(epoch_id)
+
+
+class TxPoolOps(BaseOps):
+    @with_user_endorsers
+    def get_pool_status(self) -> TxPoolStatus:
+        """
+        获取交易池状态
+        :return:
+        """
+        self._info("获取交易池状态")
+        return self._cc.get_pool_status()
+
+    @with_user_endorsers
+    def get_tx_ids_by_type_and_stage(self, tx_type: Union[TxType, str, int] = None,
+                                     tx_stage: Union[TxStage, str, int] = None) -> List[str]:
+        """
+        获取不同交易类型和阶段中的交易Id列表。
+        :param tx_type: 交易类型 在pb的txpool包中进行了定义
+        :param tx_stage: 交易阶段 在pb的txpool包中进行了定义
+        :return: 交易Id列表
+        """
+        self._info(f"获取交易类型 {tx_type} 和阶段 {tx_stage} 中的交易Id列表")
+        return self._cc.get_tx_ids_by_type_and_stage(tx_type, tx_stage)
+
+    @with_user_endorsers
+    def get_txs_in_pool_by_tx_ids(self, tx_ids: List[str]) -> (List[Transaction], List[str]):
+        """
+        根据txIds获取交易池中存在的txs，并返回交易池缺失的tx的txIds
+        :param tx_ids: 交易Id列表
+        :return: [交易池中存在的txs, 交易池缺失的tx的txIds]
+        """
+        self._info(f"根据tx_ids {tx_ids} 获取交易池中存在的txs")
+        return self._cc.get_txs_in_pool_by_tx_ids(tx_ids)
+
+    def get_tx_status(self, tx_id: str):
+        self._info(f"获取交易池中交易 {tx_id} 状态")
+        return self._cc.get_tx_status(tx_id)
+
+
+class ConsensusOps(BaseOps):
+    """共识状态操作"""
+
+    def get_consensus_validators(self) -> List[str]:
+        """
+        获取所有共识节点的身份标识
+        :return: 共识节点身份标识
+        :exception: 当查询的节点非共识节点时或共识节点内部查询中出现错误，返回error
+        """
+        self._info("获取所有共识节点的身份标识")
+        return self._cc.get_consensus_validators()
+
+    def get_consensus_height(self) -> int:
+        """
+        获取节点正在共识的区块高度
+        :return:
+        """
+        self._info("获取节点正在共识的区块高度")
+        return self._cc.get_consensus_height()
+
+    def get_consensus_state_json(self) -> dict:
+        """
+        获取共识节点的状态
+        :return: 查询的共识节点状态
+        """
+        self._info("获取共识节点的状态")
+        return self._cc.get_consensus_state_json()
+
+
 class NodeSyncCheckOps(BaseOps):
     def _get_node_clients(self, nodes: List[str] = None):
         if nodes is None:
             nodes = ['node1', 'node2', 'node3', 'node4']
         clients = [self._crypto_config.new_chain_client(conn_node=node) for node in
                    nodes]
         return clients
@@ -2821,14 +3129,19 @@
         self.private_compute = PrivateComputeOps(self._cc, self.crypto_config)  # 06
         self.dpos_erc20 = DposErc20Ops(self._cc, self.crypto_config)  # 07
         self.dpos_stake = DposStakeOps(self._cc, self.crypto_config)  # 08
         self.subscribe_manage = SubscribeManageOps(self._cc, self.crypto_config)  # 09
         self.archive_manage = ArchiveManageOps(self._cc, self.crypto_config)  # 10
         self.pubkey_manage = PubkeyManageOps(self._cc, self.crypto_config)  # 12
         self.account_manager = AccountManagerOps(self._cc, self.crypto_config)  # 13
+        self.dpos_slashing = DposSlashingOps(self._cc, self.crypto_config)  # 15
+        self.dpos_distribution = DposDistributionOps(self._cc, self.crypto_config)
+
+        self.txpool = TxPoolOps(self._cc, self.crypto_config)
+        self.consensus = ConsensusOps(self._cc, self.crypto_config)
 
         self.node_sync = NodeSyncCheckOps(self._cc, self.crypto_config)
 
         self.cmc = cmc_utils.Cmc(auth_type=self._cc.auth_type)
 
         self._cluster = None
```

### Comparing `chainmaker-2.3.2/chainmaker/client_node.py` & `chainmaker-3.0.0/chainmaker/client_node.py`

 * *Files identical despite different names*

### Comparing `chainmaker-2.3.2/chainmaker/client_user.py` & `chainmaker-3.0.0/chainmaker/client_user.py`

 * *Files identical despite different names*

### Comparing `chainmaker-2.3.2/chainmaker/conn_pool.py` & `chainmaker-3.0.0/chainmaker/conn_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,20 +165,20 @@
         if retry_interval is None:
             retry_interval = DefaultConfig.rpc_retry_interval
 
         err_msg = ''
         for i in range(retry_limit):
             try:
                 return self.get_client(conn_node).SendRequest(tx_request, timeout=timeout)
-            except grpc._channel._InactiveRpcError as ex:
+            except grpc.RpcError as ex:
                 # todo 处理 DeadlineExceeded
                 err_msg = ERR_MSG_MAP.get(ex.details(), ex.details())
                 # self._logger.exception(ex)
                 time.sleep(retry_interval // 1000)  # 毫秒
-                self._logger.debug('[Sdk] %s: retry to send rpc request to %s' % (ex.details(), self.node.node_addr))
+                self._logger.debug('[Sdk] retry to send rpc request to %s' % self.node.node_addr)
 
         else:
             raise RpcConnectError(
                 '[Sdk] rpc service<%s enable_tls=%s> not available: %s' % (
                     self.node.node_addr, self.node.enable_tls, err_msg))
 
     def close(self):
```

### Comparing `chainmaker-2.3.2/chainmaker/exceptions.py` & `chainmaker-3.0.0/chainmaker/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # @FileName     :   exceptions.py
 # @Function     :   已知异常
 
 # InactiveRpcError = grpc._channel._InactiveRpcError
+from chainmaker.protos.common.result_pb2 import TxStatusCode
 
 ERR_MSG_MAP = {
     'Empty switch_branch': 'Empty trust_root_paths',
     'failed to connect to all addresses': 'Failed to connect address, please check server, port and trust_root_paths'
 }
 
 
@@ -277,28 +278,26 @@
 # verify admin failed
 #  'the method does not found'
 # account address is illegal
 # signers do not meet the requirements (ARCHIVE)
 
 
 def handle_internal_error(tx_response):
-    pass
-    # if 'tx verify failed' in tx_response.message:
-    #     if 'is forbidden to access' in tx_response.message:
-    #         raise ForbiddenAccessError(TxStatusCode.Name(tx_response.code), tx_response.message)
-    #     if 'not enough participants' in tx_response.message:
-    #         raise EndorsementNotEnoughError(TxStatusCode.Name(tx_response.code), tx_response.message)
-    #     if 'endorsement is nil' in tx_response.message:
-    #         raise EndorsementEmptyError(TxStatusCode.Name(tx_response.code), tx_response.message)
-    #     if 'refine endorsements failed' in tx_response.message:
-    #         raise EndorsementInvalidError(TxStatusCode.Name(tx_response.code), tx_response.message)
-    #     raise AuthenticationError(TxStatusCode.Name(tx_response.code), tx_response.message)
-    # if 'TxPool is full' in tx_response.message:
-    #     raise TxPoolFullError(TxStatusCode.Name(tx_response.code), tx_response.message)
+    if 'tx verify failed' in tx_response.message:
+        if 'is forbidden to access' in tx_response.message:
+            raise ForbiddenAccessError(TxStatusCode.Name(tx_response.code), tx_response.message)
+        if 'not enough participants' in tx_response.message:
+            raise EndorsementNotEnoughError(TxStatusCode.Name(tx_response.code), tx_response.message)
+        if 'endorsement is nil' in tx_response.message:
+            raise EndorsementEmptyError(TxStatusCode.Name(tx_response.code), tx_response.message)
+        if 'refine endorsements failed' in tx_response.message:
+            raise EndorsementInvalidError(TxStatusCode.Name(tx_response.code), tx_response.message)
+        raise AuthenticationError(TxStatusCode.Name(tx_response.code), tx_response.message)
+    if 'TxPool is full' in tx_response.message:
+        raise TxPoolFullError(TxStatusCode.Name(tx_response.code), tx_response.message)
 
 
 def handle_contract_fail(tx_response):
-    pass
-    # if 'gas limit is not enough' in tx_response.message:
-    #     raise GasLimitNotEnoughError(TxStatusCode.Name(tx_response.code), tx_response.message)
-    # if 'contract initial fail' in tx_response.message:
-    #     raise ContractInitialError(TxStatusCode.Name(tx_response.code), tx_response.message)
+    if 'gas limit is not enough' in tx_response.message:
+        raise GasLimitNotEnoughError(TxStatusCode.Name(tx_response.code), tx_response.message)
+    if 'contract initial fail' in tx_response.message:
+        raise ContractInitialError(TxStatusCode.Name(tx_response.code), tx_response.message)
```

### Comparing `chainmaker-2.3.2/chainmaker/keys.py` & `chainmaker-3.0.0/chainmaker/keys.py`

 * *Files identical despite different names*

### Comparing `chainmaker-2.3.2/chainmaker/payload.py` & `chainmaker-3.0.0/chainmaker/payload.py`

 * *Files identical despite different names*

### Comparing `chainmaker-2.3.2/chainmaker/sdk_config.py` & `chainmaker-3.0.0/chainmaker/sdk_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,19 +351,19 @@
     subscribe_timeout = 60 * 10  # 订阅等待区块超时时间, 单位, 秒
     check_cert_timeout = 30
 
     with_sync_result = True  #
     with_rwset = False
 
     # rpc链接
-    rpc_retry_interval = 1000  # 获取可用客户端连接对象重试时间间隔，单位：ms
-    rpc_retry_limit = 60  # 获取可用客户端连接对象最大重试次数
+    rpc_retry_interval = 500  # 获取可用客户端连接对象重试时间间隔，单位：ms
+    rpc_retry_limit = 3  # 获取可用客户端连接对象最大重试次数
 
     retry_limit = 90  # 同步交易结果模式下，轮询获取交易结果时的最大轮询次数，删除此项或设为<=0则使用默认值 60 (sdk-go默认为30)
-    retry_interval = 1000  # 同步交易结果模式下，每次轮询交易结果时的等待时间，单位：ms 删除此项或设为<=0则使用默认值 500
+    retry_interval = 500  # 同步交易结果模式下，每次轮询交易结果时的等待时间，单位：ms 删除此项或设为<=0则使用默认值 500
     # 额外
     retry_timeout = 90  # 同步交易结果模式下，轮询获取交易结果时的最大轮询超时时间，单位秒, 和retry_limit二选一，默认30s
 
     wait_chainmaker_ok_timeout = 60
     wait_chainmaker_ok_interval = 1000
 
     txpool_full_retry_timeout = 60
```

### Comparing `chainmaker-2.3.2/setup.py` & `chainmaker-3.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,55 +3,40 @@
 # Copyright (C) THL A29 Limited, a Tencent company. All rights reserved.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # @FileName     :   setup.py
 # @Function     :   安装配置
 
-from setuptools import setup, find_packages
+from setuptools import setup
 
-__VERSION__ = '2.3.2'
-__AUTHOR__ = 'The THL chainmaker developers'
-__AUTHOR_EMAIL = 'operation@chainmaker.org'
-
-INSTALL_REQUIRES = [
-    "protobuf",
-    "grpcio",
-    "pyyaml",
-    "cryptography",
-    "pysha3",
-    "pymysql",
-    "eth-abi",
-    "asn1",
-    "pyasn1",
-    "pyasn1-modules"
-]
+# VERSION = '2.3.1'
+VERSION = '3.0.0'
 
 setup(
     name='chainmaker',
-    description='ChainMaker Python SDK',
-    version=__VERSION__,
-    author=__AUTHOR__,
-    author_email=__AUTHOR_EMAIL,
-    license='Apache-2.0',
+    version=VERSION,
+    packages=['chainmaker',
+              'chainmaker.utils',
+              'chainmaker.utils.gm',
+              'chainmaker.apis',
+              'chainmaker.protos',
+              'chainmaker.protos.accesscontrol',
+              'chainmaker.protos.api',
+              'chainmaker.protos.common',
+              'chainmaker.protos.config',
+              'chainmaker.protos.consensus',
+              'chainmaker.protos.discovery',
+              'chainmaker.protos.net',
+              'chainmaker.protos.store',
+              'chainmaker.protos.sync',
+              'chainmaker.protos.syscontract',
+              'chainmaker.protos.txpool',
+              ],
     url='https://git.chainmaker.org.cn/chainmaker/chainmaker-sdk-python.git',
-    install_requires=INSTALL_REQUIRES,
-    include_package_data=True,
-    packages=find_packages(include=['chainmaker']),
-    # packages=['chainmaker',
-    #           'chainmaker.utils',
-    #           'chainmaker.utils.gm',
-    #           'chainmaker.apis',
-    #           'chainmaker.protos',
-    #           'chainmaker.protos.accesscontrol',
-    #           'chainmaker.protos.api',
-    #           'chainmaker.protos.common',
-    #           'chainmaker.protos.config',
-    #           'chainmaker.protos.consensus',
-    #           'chainmaker.protos.discovery',
-    #           'chainmaker.protos.net',
-    #           'chainmaker.protos.store',
-    #           'chainmaker.protos.sync',
-    #           'chainmaker.protos.syscontract',
-    #           'chainmaker.protos.txpool',
-    #           ],
+    license='Apache-2.0',
+    author='The THL chainmaker developers',
+    author_email='operation@chainmaker.org',
+    description='ChainMaker Python SDK',
+    install_requires=["protobuf", "grpcio", "pyyaml", "cryptography", "pysha3", "pymysql", "eth-abi",
+                      "asn1", "pyasn1", "pyasn1-modules"]
 )
```

