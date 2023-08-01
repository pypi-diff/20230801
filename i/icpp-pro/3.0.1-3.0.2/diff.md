# Comparing `tmp/icpp-pro-3.0.1.tar.gz` & `tmp/icpp-pro-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icpp-pro-3.0.1.tar", last modified: Mon Jul 17 19:47:31 2023, max compression
+gzip compressed data, was "icpp-pro-3.0.2.tar", last modified: Tue Aug  1 19:21:27 2023, max compression
```

## Comparing `icpp-pro-3.0.1.tar` & `icpp-pro-3.0.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.639213 icpp-pro-3.0.1/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1066 2023-07-17 00:47:35.000000 icpp-pro-3.0.1/LICENSE
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1354 2023-07-17 19:47:31.639213 icpp-pro-3.0.1/PKG-INFO
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      541 2023-07-17 19:46:10.000000 icpp-pro-3.0.1/README.md
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      450 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/pyproject.toml
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       38 2023-07-17 19:47:31.639213 icpp-pro-3.0.1/setup.cfg
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    10118 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/setup.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.615213 icpp-pro-3.0.1/src/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.623213 icpp-pro-3.0.1/src/icpp/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      747 2023-04-29 11:50:55.000000 icpp-pro-3.0.1/src/icpp/__init__.py
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1086 2023-05-19 20:47:09.000000 icpp-pro-3.0.1/src/icpp/__main__.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.615213 icpp-pro-3.0.1/src/icpp/canisters/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.623213 icpp-pro-3.0.1/src/icpp/canisters/greet/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)       92 2023-04-29 11:50:55.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/README.md
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3389 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/demo.ps1
--rwxr-xr-x   0 arjaan    (1000) arjaan    (1000)     2404 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/demo.sh
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      232 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/dfx.json
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      474 2023-04-29 11:50:55.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/icpp.toml
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.623213 icpp-pro-3.0.1/src/icpp/canisters/greet/native/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3297 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/native/main.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      137 2023-05-19 20:47:09.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/native/main.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.627213 icpp-pro-3.0.1/src/icpp/canisters/greet/src/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     5411 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/src/greet.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      599 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/src/greet.did
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      427 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/src/greet.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.627213 icpp-pro-3.0.1/src/icpp/canisters/greet/test/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        0 2023-04-29 11:50:55.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/test/__init__.py
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      298 2023-04-29 11:50:55.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/test/conftest.py
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3723 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/canisters/greet/test/test_apis.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     8258 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/src/icpp/commands_build_native.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7957 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/commands_build_wasm.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1122 2023-04-29 11:50:55.000000 icpp-pro-3.0.1/src/icpp/commands_get.py
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      753 2023-04-29 11:50:55.000000 icpp-pro-3.0.1/src/icpp/commands_init.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4804 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/commands_install_wasi_sdk.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     6097 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/config_default.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2991 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/src/icpp/conftest_base.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3558 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/decorators.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.615213 icpp-pro-3.0.1/src/icpp/ic/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.631213 icpp-pro-3.0.1/src/icpp/ic/canister/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1288 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      405 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_base.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1389 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_base.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      292 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_cleanup_callback.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      240 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_cleanup_callback.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      268 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_global_timer.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      224 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_global_timer.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      256 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_heartbeat.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      216 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_heartbeat.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      226 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_init.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      196 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_init.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      286 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_inspect_message.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      236 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_inspect_message.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      268 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_post_upgrade.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      224 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_post_upgrade.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      262 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_pre_upgrade.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      220 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_pre_upgrade.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      232 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_query.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      200 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_query.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      286 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_reject_callback.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      236 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_reject_callback.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      280 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_reply_callback.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      232 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_reply_callback.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      232 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_start.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      200 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_start.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      238 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_update.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      204 2023-06-14 01:34:03.000000 icpp-pro-3.0.1/src/icpp/ic/canister/canister_update.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.631213 icpp-pro-3.0.1/src/icpp/ic/ic0/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3407 2023-04-29 11:50:56.000000 icpp-pro-3.0.1/src/icpp/ic/ic0/ic0.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.635213 icpp-pro-3.0.1/src/icpp/ic/ic0mock/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      111 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/ic0mock/global.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     8131 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/src/icpp/ic/ic0mock/ic0.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2091 2023-04-29 11:50:56.000000 icpp-pro-3.0.1/src/icpp/ic/ic0mock/ic0.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4022 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/src/icpp/ic/ic0mock/mock_ic.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      157 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/ic0mock/mock_ic.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1514 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/ic0mock/mock_ic_.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.635213 icpp-pro-3.0.1/src/icpp/ic/icapi/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     6705 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/icapi/ic_api.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     8460 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/ic/icapi/ic_api.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      463 2023-04-29 11:50:56.000000 icpp-pro-3.0.1/src/icpp/ic/icapi/wasm_symbol.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.635213 icpp-pro-3.0.1/src/icpp/ic/pro/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      816 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/src/icpp/ic/pro/pro.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      393 2023-04-29 17:59:16.000000 icpp-pro-3.0.1/src/icpp/ic/pro/pro.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.635213 icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1370 2023-04-29 11:50:56.000000 icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/__wasilibc_initialize_environ.c
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      327 2023-04-29 11:50:56.000000 icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/ic_trap.c
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       70 2023-04-29 11:50:56.000000 icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/ic_trap.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4743 2023-05-19 20:47:09.000000 icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/posix.c
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    10198 2023-05-19 20:47:09.000000 icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/unreachable.c
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4002 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/icpp_toml.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      670 2023-05-19 20:47:09.000000 icpp-pro-3.0.1/src/icpp/options_build.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      923 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/src/icpp/options_main.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      866 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/src/icpp/pro.py
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       98 2023-04-29 11:50:55.000000 icpp-pro-3.0.1/src/icpp/py.typed
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5578 2023-07-17 02:27:26.000000 icpp-pro-3.0.1/src/icpp/run_shell_cmd.py
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5441 2023-07-17 19:44:47.000000 icpp-pro-3.0.1/src/icpp/smoketest.py
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      322 2023-07-17 19:47:10.000000 icpp-pro-3.0.1/src/icpp/version.py
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      231 2023-07-08 00:43:35.000000 icpp-pro-3.0.1/src/icpp/version_wasi_sdk.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 19:47:31.639213 icpp-pro-3.0.1/src/icpp_pro.egg-info/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1354 2023-07-17 19:47:31.000000 icpp-pro-3.0.1/src/icpp_pro.egg-info/PKG-INFO
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2942 2023-07-17 19:47:31.000000 icpp-pro-3.0.1/src/icpp_pro.egg-info/SOURCES.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        1 2023-07-17 19:47:31.000000 icpp-pro-3.0.1/src/icpp_pro.egg-info/dependency_links.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       44 2023-07-17 19:47:31.000000 icpp-pro-3.0.1/src/icpp_pro.egg-info/entry_points.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      136 2023-07-17 19:47:31.000000 icpp-pro-3.0.1/src/icpp_pro.egg-info/requires.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        5 2023-07-17 19:47:31.000000 icpp-pro-3.0.1/src/icpp_pro.egg-info/top_level.txt
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.116558 icpp-pro-3.0.2/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1066 2023-07-17 00:47:35.000000 icpp-pro-3.0.2/LICENSE
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1354 2023-08-01 19:21:27.112558 icpp-pro-3.0.2/PKG-INFO
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      541 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/README.md
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      450 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/pyproject.toml
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       38 2023-08-01 19:21:27.116558 icpp-pro-3.0.2/setup.cfg
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    10118 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/setup.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.096558 icpp-pro-3.0.2/src/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.100558 icpp-pro-3.0.2/src/icpp/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      747 2023-04-29 11:50:55.000000 icpp-pro-3.0.2/src/icpp/__init__.py
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1086 2023-05-19 20:47:09.000000 icpp-pro-3.0.2/src/icpp/__main__.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.096558 icpp-pro-3.0.2/src/icpp/canisters/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.104558 icpp-pro-3.0.2/src/icpp/canisters/greet/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)       92 2023-04-29 11:50:55.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/README.md
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3389 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/demo.ps1
+-rwxr-xr-x   0 arjaan    (1000) arjaan    (1000)     2404 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/demo.sh
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      232 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/dfx.json
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      474 2023-04-29 11:50:55.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/icpp.toml
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.104558 icpp-pro-3.0.2/src/icpp/canisters/greet/native/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3297 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/native/main.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      137 2023-05-19 20:47:09.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/native/main.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.104558 icpp-pro-3.0.2/src/icpp/canisters/greet/src/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     5411 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/src/greet.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      599 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/src/greet.did
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      427 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/src/greet.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.104558 icpp-pro-3.0.2/src/icpp/canisters/greet/test/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        0 2023-04-29 11:50:55.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/test/__init__.py
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      330 2023-08-01 11:27:45.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/test/conftest.py
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3723 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/canisters/greet/test/test_apis.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     8258 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/src/icpp/commands_build_native.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7957 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/commands_build_wasm.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1122 2023-04-29 11:50:55.000000 icpp-pro-3.0.2/src/icpp/commands_get.py
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      753 2023-04-29 11:50:55.000000 icpp-pro-3.0.2/src/icpp/commands_init.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4804 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/commands_install_wasi_sdk.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     6097 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/config_default.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2991 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/src/icpp/conftest_base.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3558 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/decorators.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.096558 icpp-pro-3.0.2/src/icpp/ic/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.108558 icpp-pro-3.0.2/src/icpp/ic/canister/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1288 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      405 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_base.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1513 2023-07-29 12:52:52.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_base.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      292 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_cleanup_callback.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      240 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_cleanup_callback.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      268 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_global_timer.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      224 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_global_timer.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      256 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_heartbeat.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      216 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_heartbeat.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      226 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_init.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      196 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_init.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      286 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_inspect_message.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      236 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_inspect_message.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      268 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_post_upgrade.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      224 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_post_upgrade.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      262 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_pre_upgrade.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      220 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_pre_upgrade.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      232 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_query.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      200 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_query.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      286 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_reject_callback.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      236 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_reject_callback.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      280 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_reply_callback.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      232 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_reply_callback.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      232 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_start.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      200 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_start.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      238 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_update.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      204 2023-06-14 01:34:03.000000 icpp-pro-3.0.2/src/icpp/ic/canister/canister_update.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.108558 icpp-pro-3.0.2/src/icpp/ic/ic0/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3407 2023-04-29 11:50:56.000000 icpp-pro-3.0.2/src/icpp/ic/ic0/ic0.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.112558 icpp-pro-3.0.2/src/icpp/ic/ic0mock/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      111 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/ic0mock/global.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     8131 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/src/icpp/ic/ic0mock/ic0.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2091 2023-04-29 11:50:56.000000 icpp-pro-3.0.2/src/icpp/ic/ic0mock/ic0.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4022 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/src/icpp/ic/ic0mock/mock_ic.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      157 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/ic0mock/mock_ic.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1514 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/ic0mock/mock_ic_.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.112558 icpp-pro-3.0.2/src/icpp/ic/icapi/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7255 2023-07-29 13:05:42.000000 icpp-pro-3.0.2/src/icpp/ic/icapi/ic_api.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     8460 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/ic/icapi/ic_api.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      463 2023-04-29 11:50:56.000000 icpp-pro-3.0.2/src/icpp/ic/icapi/wasm_symbol.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.112558 icpp-pro-3.0.2/src/icpp/ic/pro/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      816 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/src/icpp/ic/pro/pro.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      393 2023-04-29 17:59:16.000000 icpp-pro-3.0.2/src/icpp/ic/pro/pro.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.112558 icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1370 2023-04-29 11:50:56.000000 icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/__wasilibc_initialize_environ.c
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      327 2023-04-29 11:50:56.000000 icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/ic_trap.c
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       70 2023-04-29 11:50:56.000000 icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/ic_trap.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4743 2023-05-19 20:47:09.000000 icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/posix.c
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    10198 2023-05-19 20:47:09.000000 icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/unreachable.c
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4002 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/icpp_toml.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      670 2023-05-19 20:47:09.000000 icpp-pro-3.0.2/src/icpp/options_build.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      923 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/src/icpp/options_main.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      866 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/src/icpp/pro.py
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       98 2023-04-29 11:50:55.000000 icpp-pro-3.0.2/src/icpp/py.typed
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5578 2023-07-17 02:27:26.000000 icpp-pro-3.0.2/src/icpp/run_shell_cmd.py
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5441 2023-07-17 19:55:55.000000 icpp-pro-3.0.2/src/icpp/smoketest.py
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      322 2023-08-01 19:19:36.000000 icpp-pro-3.0.2/src/icpp/version.py
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      231 2023-07-08 00:43:35.000000 icpp-pro-3.0.2/src/icpp/version_wasi_sdk.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:21:27.112558 icpp-pro-3.0.2/src/icpp_pro.egg-info/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1354 2023-08-01 19:21:27.000000 icpp-pro-3.0.2/src/icpp_pro.egg-info/PKG-INFO
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2942 2023-08-01 19:21:27.000000 icpp-pro-3.0.2/src/icpp_pro.egg-info/SOURCES.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        1 2023-08-01 19:21:27.000000 icpp-pro-3.0.2/src/icpp_pro.egg-info/dependency_links.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       44 2023-08-01 19:21:27.000000 icpp-pro-3.0.2/src/icpp_pro.egg-info/entry_points.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      136 2023-08-01 19:21:27.000000 icpp-pro-3.0.2/src/icpp_pro.egg-info/requires.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        5 2023-08-01 19:21:27.000000 icpp-pro-3.0.2/src/icpp_pro.egg-info/top_level.txt
```

### Comparing `icpp-pro-3.0.1/LICENSE` & `icpp-pro-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/PKG-INFO` & `icpp-pro-3.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-pro
-Version: 3.0.1
+Version: 3.0.2
 Summary: C++ Canister Development Kit (CDK) for the Internet Computer
 Home-page: https://docs.icpp.world/
 Author: icpp team
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: Internet Computer,C++,Canister Development Kit,CDK,Smart Contracts,blockchain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `icpp-pro-3.0.1/README.md` & `icpp-pro-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/setup.py` & `icpp-pro-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/__init__.py` & `icpp-pro-3.0.2/src/icpp/__init__.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/__main__.py` & `icpp-pro-3.0.2/src/icpp/__main__.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/canisters/greet/demo.ps1` & `icpp-pro-3.0.2/src/icpp/canisters/greet/demo.ps1`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/canisters/greet/demo.sh` & `icpp-pro-3.0.2/src/icpp/canisters/greet/demo.sh`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/canisters/greet/native/main.cpp` & `icpp-pro-3.0.2/src/icpp/canisters/greet/native/main.cpp`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/canisters/greet/src/greet.cpp` & `icpp-pro-3.0.2/src/icpp/canisters/greet/src/greet.cpp`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/canisters/greet/src/greet.did` & `icpp-pro-3.0.2/src/icpp/canisters/greet/src/greet.did`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/canisters/greet/test/test_apis.py` & `icpp-pro-3.0.2/src/icpp/canisters/greet/test/test_apis.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/commands_build_native.py` & `icpp-pro-3.0.2/src/icpp/commands_build_native.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/commands_build_wasm.py` & `icpp-pro-3.0.2/src/icpp/commands_build_wasm.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/commands_get.py` & `icpp-pro-3.0.2/src/icpp/commands_get.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/commands_init.py` & `icpp-pro-3.0.2/src/icpp/commands_init.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/commands_install_wasi_sdk.py` & `icpp-pro-3.0.2/src/icpp/commands_install_wasi_sdk.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/config_default.py` & `icpp-pro-3.0.2/src/icpp/config_default.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/conftest_base.py` & `icpp-pro-3.0.2/src/icpp/conftest_base.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/decorators.py` & `icpp-pro-3.0.2/src/icpp/decorators.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/canister/canister.h` & `icpp-pro-3.0.2/src/icpp/ic/canister/canister.h`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/canister/canister_base.h` & `icpp-pro-3.0.2/src/icpp/ic/canister/canister_base.h`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,16 @@
   bool is_entry_s() { return m_entry_type == "CanisterStart"; }
   bool is_entry_F() { return m_entry_type == "CanisterInspectMessage"; }
   bool is_entry_T() {
     return m_entry_type == "CanisterHeartbeat" ||
            m_entry_type == "CanisterGlobalTimer";
   }
   bool is_entry_Wildcard() { return m_entry_type != "CanisterStart"; }
+  std::string get_calling_function() { return m_calling_function; }
+  std::string get_entry_type() { return m_entry_type; }
 
 protected:
   // The calling function
   std::string m_calling_function{""};
   // The entry type
   std::string m_entry_type{"CanisterQuery"};
 };
```

### Comparing `icpp-pro-3.0.1/src/icpp/ic/ic0/ic0.h` & `icpp-pro-3.0.2/src/icpp/ic/ic0/ic0.h`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/ic0mock/ic0.cpp` & `icpp-pro-3.0.2/src/icpp/ic/ic0mock/ic0.cpp`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/ic0mock/ic0.h` & `icpp-pro-3.0.2/src/icpp/ic/ic0mock/ic0.h`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/ic0mock/mock_ic.cpp` & `icpp-pro-3.0.2/src/icpp/ic/ic0mock/mock_ic.cpp`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/ic0mock/mock_ic_.h` & `icpp-pro-3.0.2/src/icpp/ic/ic0mock/mock_ic_.h`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/icapi/ic_api.cpp` & `icpp-pro-3.0.2/src/icpp/ic/icapi/ic_api.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -192,14 +192,23 @@
   to_wire(args_out);
 }
 
 void IC_API::to_wire(const CandidArgs &args_out) {
   if (m_called_to_wire) {
     trap("ERROR: The canister is calling ic_api.to_wire() more than once.");
   }
+  if (!(m_canister_entry.is_entry_U() || m_canister_entry.is_entry_Q() ||
+        m_canister_entry.is_entry_Ry() || m_canister_entry.is_entry_Rt())) {
+    trap(
+        "ERROR: The canister function '" +
+        m_canister_entry.get_calling_function() +
+        "' is calling ic_api.to_wire(), but it is of type '" +
+        m_canister_entry.get_entry_type() +
+        "'.\nYou can only call ic_api.to_wire() for CanisterQuery, CanisterUpdate, CanisterReplyCallback & CanisterRejectCallback functions.\nPlease update the IC_API instantiation.");
+  }
   m_called_to_wire = true;
 
   m_B_out = CandidSerialize(args_out).get_B();
 
   // Optionally, debug print the final result
   if (m_debug_print) {
     debug_print("\n--");
```

### Comparing `icpp-pro-3.0.1/src/icpp/ic/icapi/ic_api.h` & `icpp-pro-3.0.2/src/icpp/ic/icapi/ic_api.h`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/pro/pro.cpp` & `icpp-pro-3.0.2/src/icpp/ic/pro/pro.cpp`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/__wasilibc_initialize_environ.c` & `icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/__wasilibc_initialize_environ.c`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/posix.c` & `icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/posix.c`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/ic/wasi_sdk_traps/unreachable.c` & `icpp-pro-3.0.2/src/icpp/ic/wasi_sdk_traps/unreachable.c`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/icpp_toml.py` & `icpp-pro-3.0.2/src/icpp/icpp_toml.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/options_build.py` & `icpp-pro-3.0.2/src/icpp/options_build.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/options_main.py` & `icpp-pro-3.0.2/src/icpp/options_main.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/pro.py` & `icpp-pro-3.0.2/src/icpp/pro.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/run_shell_cmd.py` & `icpp-pro-3.0.2/src/icpp/run_shell_cmd.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp/smoketest.py` & `icpp-pro-3.0.2/src/icpp/smoketest.py`

 * *Files identical despite different names*

### Comparing `icpp-pro-3.0.1/src/icpp_pro.egg-info/PKG-INFO` & `icpp-pro-3.0.2/src/icpp_pro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-pro
-Version: 3.0.1
+Version: 3.0.2
 Summary: C++ Canister Development Kit (CDK) for the Internet Computer
 Home-page: https://docs.icpp.world/
 Author: icpp team
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: Internet Computer,C++,Canister Development Kit,CDK,Smart Contracts,blockchain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `icpp-pro-3.0.1/src/icpp_pro.egg-info/SOURCES.txt` & `icpp-pro-3.0.2/src/icpp_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

